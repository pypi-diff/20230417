# Comparing `tmp/goastpy-0.1.1.tar.gz` & `tmp/goastpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goastpy-0.1.1.tar", last modified: Sun Apr 16 13:05:44 2023, max compression
+gzip compressed data, was "goastpy-0.1.3.tar", last modified: Mon Apr 17 07:59:31 2023, max compression
```

## Comparing `goastpy-0.1.1.tar` & `goastpy-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-16 13:05:44.488643 goastpy-0.1.1/
--rw-r--r--   0 monolite   (502) staff       (20)     1064 2023-04-16 11:48:27.000000 goastpy-0.1.1/LICENSE
--rw-r--r--   0 monolite   (502) staff       (20)      774 2023-04-16 13:05:44.488742 goastpy-0.1.1/PKG-INFO
--rw-r--r--   0 monolite   (502) staff       (20)       54 2023-04-16 11:48:27.000000 goastpy-0.1.1/README.md
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-16 13:05:44.488520 goastpy-0.1.1/goastpy.egg-info/
--rw-r--r--   0 monolite   (502) staff       (20)      774 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/PKG-INFO
--rw-r--r--   0 monolite   (502) staff       (20)      160 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/SOURCES.txt
--rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/dependency_links.txt
--rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/top_level.txt
--rw-r--r--   0 monolite   (502) staff       (20)       79 2023-04-16 13:05:44.489035 goastpy-0.1.1/setup.cfg
--rw-r--r--   0 monolite   (502) staff       (20)      903 2023-04-16 13:05:42.000000 goastpy-0.1.1/setup.py
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 07:59:31.239636 goastpy-0.1.3/
+-rw-r--r--   0 monolite   (502) staff       (20)     1064 2023-04-16 11:48:27.000000 goastpy-0.1.3/LICENSE
+-rw-r--r--   0 monolite   (502) staff       (20)      897 2023-04-17 07:59:31.239740 goastpy-0.1.3/PKG-INFO
+-rw-r--r--   0 monolite   (502) staff       (20)       54 2023-04-16 11:48:27.000000 goastpy-0.1.3/README.md
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 07:59:31.238745 goastpy-0.1.3/goastpy/
+-rw-r--r--   0 monolite   (502) staff       (20)       27 2023-04-16 13:44:10.000000 goastpy-0.1.3/goastpy/__init__.py
+-rw-r--r--   0 monolite   (502) staff       (20)     3298 2023-04-17 07:48:55.000000 goastpy-0.1.3/goastpy/goastparser_wrapper.py
+-rw-r--r--   0 monolite   (502) staff       (20)      687 2023-04-16 13:44:59.000000 goastpy-0.1.3/goastpy/goastpy.py
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-17 07:59:31.239473 goastpy-0.1.3/goastpy.egg-info/
+-rw-r--r--   0 monolite   (502) staff       (20)      897 2023-04-17 07:59:31.000000 goastpy-0.1.3/goastpy.egg-info/PKG-INFO
+-rw-r--r--   0 monolite   (502) staff       (20)      230 2023-04-17 07:59:31.000000 goastpy-0.1.3/goastpy.egg-info/SOURCES.txt
+-rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-17 07:59:31.000000 goastpy-0.1.3/goastpy.egg-info/dependency_links.txt
+-rw-r--r--   0 monolite   (502) staff       (20)        8 2023-04-17 07:59:31.000000 goastpy-0.1.3/goastpy.egg-info/top_level.txt
+-rw-r--r--   0 monolite   (502) staff       (20)       79 2023-04-17 07:59:31.240188 goastpy-0.1.3/setup.cfg
+-rw-r--r--   0 monolite   (502) staff       (20)     1046 2023-04-17 07:59:22.000000 goastpy-0.1.3/setup.py
```

### Comparing `goastpy-0.1.1/LICENSE` & `goastpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.1/PKG-INFO` & `goastpy-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.1
+Version: 0.1.3
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
-Download-URL: https://github.com/itayg25/goastpy/archive/v_01.tar.gz
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
-License: MIT
-Keywords: GO,GOLANG,PYTHON,AST,GOPYGO
+Keywords: GO,GOLANG,PYTHON,AST,GOPY,PYGO,PARSER,ASTPARSER
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# gopyast
+a python wrapper for the built-in go parser
```

### Comparing `goastpy-0.1.1/goastpy.egg-info/PKG-INFO` & `goastpy-0.1.3/goastpy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.1
+Version: 0.1.3
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
-Download-URL: https://github.com/itayg25/goastpy/archive/v_01.tar.gz
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
-License: MIT
-Keywords: GO,GOLANG,PYTHON,AST,GOPYGO
+Keywords: GO,GOLANG,PYTHON,AST,GOPY,PYGO,PARSER,ASTPARSER
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# gopyast
+a python wrapper for the built-in go parser
```

### Comparing `goastpy-0.1.1/setup.py` & `goastpy-0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='goastpy',
-    packages=find_packages(),
-    version='0.1.1',
-    license='MIT',
+    name="goastpy",
+    version="0.1.3",
+    packages=["goastpy"],
+    install_requires=[],
     description='a python wrapper for the built-in go parser using c-types',
     author='Itay Gersten',
     author_email='Itay.Gersten@gmail.com',
     url='https://github.com/itayg25/goastpy',
-    download_url='https://github.com/itayg25/goastpy/archive/v_01.tar.gz',
-    keywords=['GO', 'GOLANG', 'PYTHON', 'AST', 'GOPYGO'],
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    keywords=['GO', 'GOLANG', 'PYTHON', 'AST', 'GOPY', 'PYGO', 'PARSER', 'ASTPARSER'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires=">=3.6",
+
 )
```

