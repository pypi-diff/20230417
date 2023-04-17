# Comparing `tmp/shogun-build-0.3.0.tar.gz` & `tmp/shogun-build-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shogun-build-0.3.0.tar", last modified: Sun Apr 16 23:50:54 2023, max compression
+gzip compressed data, was "shogun-build-0.3.1.tar", last modified: Mon Apr 17 00:00:28 2023, max compression
```

## Comparing `shogun-build-0.3.0.tar` & `shogun-build-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-16 23:50:54.895357 shogun-build-0.3.0/
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1271 2022-08-06 19:20:48.000000 shogun-build-0.3.0/LICENSE
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1488 2023-04-16 23:50:54.895357 shogun-build-0.3.0/PKG-INFO
--rw-r--r--   0 branalba  (1000) branalba  (1000)      582 2023-03-14 20:47:36.000000 shogun-build-0.3.0/README.md
--rw-r--r--   0 branalba  (1000) branalba  (1000)      285 2023-04-16 23:49:48.000000 shogun-build-0.3.0/pyproject.toml
--rw-r--r--   0 branalba  (1000) branalba  (1000)       38 2023-04-16 23:50:54.895357 shogun-build-0.3.0/setup.cfg
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-16 23:50:54.895357 shogun-build-0.3.0/shogun/
--rw-r--r--   0 branalba  (1000) branalba  (1000)        0 2022-08-03 19:14:34.000000 shogun-build-0.3.0/shogun/__init__.py
--rw-r--r--   0 branalba  (1000) branalba  (1000)     6130 2023-01-11 18:39:50.000000 shogun-build-0.3.0/shogun/buildutils.py
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1907 2022-08-19 03:54:16.000000 shogun-build-0.3.0/shogun/pathutil.py
--rw-r--r--   0 branalba  (1000) branalba  (1000)     3657 2022-08-24 19:04:05.000000 shogun-build-0.3.0/shogun/platforms.py
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-16 23:50:54.895357 shogun-build-0.3.0/shogun/thirdparty/
--rw-r--r--   0 branalba  (1000) branalba  (1000)     6946 2022-08-06 18:24:39.000000 shogun-build-0.3.0/shogun/thirdparty/ninja_syntax.py
-drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-16 23:50:54.895357 shogun-build-0.3.0/shogun_build.egg-info/
--rw-r--r--   0 branalba  (1000) branalba  (1000)     1488 2023-04-16 23:50:54.000000 shogun-build-0.3.0/shogun_build.egg-info/PKG-INFO
--rw-r--r--   0 branalba  (1000) branalba  (1000)      324 2023-04-16 23:50:54.000000 shogun-build-0.3.0/shogun_build.egg-info/SOURCES.txt
--rw-r--r--   0 branalba  (1000) branalba  (1000)        1 2023-04-16 23:50:54.000000 shogun-build-0.3.0/shogun_build.egg-info/dependency_links.txt
--rw-r--r--   0 branalba  (1000) branalba  (1000)        6 2023-04-16 23:50:54.000000 shogun-build-0.3.0/shogun_build.egg-info/requires.txt
--rw-r--r--   0 branalba  (1000) branalba  (1000)        7 2023-04-16 23:50:54.000000 shogun-build-0.3.0/shogun_build.egg-info/top_level.txt
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     1063 2023-04-17 00:00:15.000000 shogun-build-0.3.1/LICENSE
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     1478 2023-04-17 00:00:28.308867 shogun-build-0.3.1/PKG-INFO
+-rw-r--r--   0 branalba  (1000) branalba  (1000)      582 2023-03-14 20:47:36.000000 shogun-build-0.3.1/README.md
+-rw-r--r--   0 branalba  (1000) branalba  (1000)      510 2023-04-16 23:59:31.000000 shogun-build-0.3.1/pyproject.toml
+-rw-r--r--   0 branalba  (1000) branalba  (1000)       38 2023-04-17 00:00:28.308867 shogun-build-0.3.1/setup.cfg
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/shogun/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        0 2022-08-03 19:14:34.000000 shogun-build-0.3.1/shogun/__init__.py
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     6130 2023-01-11 18:39:50.000000 shogun-build-0.3.1/shogun/buildutils.py
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     1907 2022-08-19 03:54:16.000000 shogun-build-0.3.1/shogun/pathutil.py
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     3657 2022-08-24 19:04:05.000000 shogun-build-0.3.1/shogun/platforms.py
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/shogun/thirdparty/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     6946 2022-08-06 18:24:39.000000 shogun-build-0.3.1/shogun/thirdparty/ninja_syntax.py
+drwxr-xr-x   0 branalba  (1000) branalba  (1000)        0 2023-04-17 00:00:28.308867 shogun-build-0.3.1/shogun_build.egg-info/
+-rw-r--r--   0 branalba  (1000) branalba  (1000)     1478 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/PKG-INFO
+-rw-r--r--   0 branalba  (1000) branalba  (1000)      324 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/SOURCES.txt
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        1 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/dependency_links.txt
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        6 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/requires.txt
+-rw-r--r--   0 branalba  (1000) branalba  (1000)        7 2023-04-17 00:00:28.000000 shogun-build-0.3.1/shogun_build.egg-info/top_level.txt
```

### Comparing `shogun-build-0.3.0/LICENSE` & `shogun-build-0.3.1/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-The following license applies to all files within this repository EXCEPT those within the folder ./shogun/thirdparty. For each of those files, their respective licenses will be indicated in the file itself.
-
-Copyright © 2021 Brandon Alba
+Copyright © 2023 Brandon Alba
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `shogun-build-0.3.0/PKG-INFO` & `shogun-build-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: shogun-build
-Version: 0.3.0
+Version: 0.3.1
+Summary: Package for facilitating the creation of Python-based build scripts using Ninja as the compilation backend. Focuses on small projects using gcc/g++.
 Author-email: Brandon Alba <brandonealba@protonmail.com>
-License: The following license applies to all files within this repository EXCEPT those within the folder ./shogun/thirdparty. For each of those files, their respective licenses will be indicated in the file itself.
-        
-        Copyright © 2021 Brandon Alba
+License: Copyright © 2023 Brandon Alba
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
+Project-URL: Source, https://github.com/branalba/shogun
 License-File: LICENSE
```

### Comparing `shogun-build-0.3.0/README.md` & `shogun-build-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.0/shogun/buildutils.py` & `shogun-build-0.3.1/shogun/buildutils.py`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.0/shogun/pathutil.py` & `shogun-build-0.3.1/shogun/pathutil.py`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.0/shogun/platforms.py` & `shogun-build-0.3.1/shogun/platforms.py`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.0/shogun/thirdparty/ninja_syntax.py` & `shogun-build-0.3.1/shogun/thirdparty/ninja_syntax.py`

 * *Files identical despite different names*

### Comparing `shogun-build-0.3.0/shogun_build.egg-info/PKG-INFO` & `shogun-build-0.3.1/shogun_build.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: shogun-build
-Version: 0.3.0
+Version: 0.3.1
+Summary: Package for facilitating the creation of Python-based build scripts using Ninja as the compilation backend. Focuses on small projects using gcc/g++.
 Author-email: Brandon Alba <brandonealba@protonmail.com>
-License: The following license applies to all files within this repository EXCEPT those within the folder ./shogun/thirdparty. For each of those files, their respective licenses will be indicated in the file itself.
-        
-        Copyright © 2021 Brandon Alba
+License: Copyright © 2023 Brandon Alba
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
+Project-URL: Source, https://github.com/branalba/shogun
 License-File: LICENSE
```

