# Comparing `tmp/merkle-py-1.2.1.tar.gz` & `tmp/merkle-py-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkle-py-1.2.1.tar", last modified: Tue Mar 14 16:53:55 2023, max compression
+gzip compressed data, was "merkle-py-1.2.2.tar", last modified: Mon Apr 17 07:03:47 2023, max compression
```

## Comparing `merkle-py-1.2.1.tar` & `merkle-py-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-14 16:53:55.754714 merkle-py-1.2.1/
--rw-r--r--   0 cyrildever   (501) staff       (20)       19 2022-03-21 11:01:19.000000 merkle-py-1.2.1/MANIFEST.in
--rw-r--r--   0 cyrildever   (501) staff       (20)     2922 2023-03-14 16:53:55.754402 merkle-py-1.2.1/PKG-INFO
--rw-r--r--   0 cyrildever   (501) staff       (20)     2435 2023-03-14 10:19:00.000000 merkle-py-1.2.1/README.md
--rw-r--r--   0 cyrildever   (501) staff       (20)      103 2022-03-21 11:01:19.000000 merkle-py-1.2.1/pyproject.toml
--rw-r--r--   0 cyrildever   (501) staff       (20)       38 2023-03-14 16:53:55.754799 merkle-py-1.2.1/setup.cfg
--rw-r--r--   0 cyrildever   (501) staff       (20)      872 2023-03-14 16:52:17.000000 merkle-py-1.2.1/setup.py
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-14 16:53:55.743832 merkle-py-1.2.1/src/
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-14 16:53:55.746654 merkle-py-1.2.1/src/merkle_py.egg-info/
--rw-r--r--   0 cyrildever   (501) staff       (20)     2922 2023-03-14 16:53:55.000000 merkle-py-1.2.1/src/merkle_py.egg-info/PKG-INFO
--rw-r--r--   0 cyrildever   (501) staff       (20)      452 2023-03-14 16:53:55.000000 merkle-py-1.2.1/src/merkle_py.egg-info/SOURCES.txt
--rw-r--r--   0 cyrildever   (501) staff       (20)        1 2023-03-14 16:53:55.000000 merkle-py-1.2.1/src/merkle_py.egg-info/dependency_links.txt
--rw-r--r--   0 cyrildever   (501) staff       (20)        9 2023-03-14 16:53:55.000000 merkle-py-1.2.1/src/merkle_py.egg-info/top_level.txt
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-14 16:53:55.750346 merkle-py-1.2.1/src/merklepy/
--rw-r--r--   0 cyrildever   (501) staff       (20)        0 2022-03-21 11:01:19.000000 merkle-py-1.2.1/src/merklepy/__init__.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      657 2022-04-04 08:47:17.000000 merkle-py-1.2.1/src/merklepy/exception.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      971 2022-04-04 08:47:17.000000 merkle-py-1.2.1/src/merklepy/hash.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      843 2022-04-04 08:47:17.000000 merkle-py-1.2.1/src/merklepy/options.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     1207 2022-04-04 08:47:17.000000 merkle-py-1.2.1/src/merklepy/path.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     2287 2022-04-04 10:31:42.000000 merkle-py-1.2.1/src/merklepy/proof.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     6813 2022-04-04 08:47:17.000000 merkle-py-1.2.1/src/merklepy/tree.py
-drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-03-14 16:53:55.753809 merkle-py-1.2.1/tests/
--rw-r--r--   0 cyrildever   (501) staff       (20)     2319 2022-04-04 08:47:17.000000 merkle-py-1.2.1/tests/test_hash.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      523 2022-04-04 08:47:17.000000 merkle-py-1.2.1/tests/test_options.py
--rw-r--r--   0 cyrildever   (501) staff       (20)      875 2022-04-04 08:47:17.000000 merkle-py-1.2.1/tests/test_path.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     1749 2022-04-04 08:47:17.000000 merkle-py-1.2.1/tests/test_proof.py
--rw-r--r--   0 cyrildever   (501) staff       (20)     5595 2022-04-04 08:47:17.000000 merkle-py-1.2.1/tests/test_tree.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-04-17 07:03:47.148045 merkle-py-1.2.2/
+-rw-r--r--   0 cyrildever   (501) staff       (20)       19 2022-03-21 11:01:19.000000 merkle-py-1.2.2/MANIFEST.in
+-rw-r--r--   0 cyrildever   (501) staff       (20)     3323 2023-04-17 07:03:47.147734 merkle-py-1.2.2/PKG-INFO
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2817 2023-04-17 06:57:59.000000 merkle-py-1.2.2/README.md
+-rw-r--r--   0 cyrildever   (501) staff       (20)      103 2022-03-21 11:01:19.000000 merkle-py-1.2.2/pyproject.toml
+-rw-r--r--   0 cyrildever   (501) staff       (20)       38 2023-04-17 07:03:47.148132 merkle-py-1.2.2/setup.cfg
+-rw-r--r--   0 cyrildever   (501) staff       (20)      902 2023-04-17 06:53:21.000000 merkle-py-1.2.2/setup.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-04-17 07:03:47.138363 merkle-py-1.2.2/src/
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-04-17 07:03:47.140862 merkle-py-1.2.2/src/merkle_py.egg-info/
+-rw-r--r--   0 cyrildever   (501) staff       (20)     3323 2023-04-17 07:03:47.000000 merkle-py-1.2.2/src/merkle_py.egg-info/PKG-INFO
+-rw-r--r--   0 cyrildever   (501) staff       (20)      452 2023-04-17 07:03:47.000000 merkle-py-1.2.2/src/merkle_py.egg-info/SOURCES.txt
+-rw-r--r--   0 cyrildever   (501) staff       (20)        1 2023-04-17 07:03:47.000000 merkle-py-1.2.2/src/merkle_py.egg-info/dependency_links.txt
+-rw-r--r--   0 cyrildever   (501) staff       (20)        9 2023-04-17 07:03:47.000000 merkle-py-1.2.2/src/merkle_py.egg-info/top_level.txt
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-04-17 07:03:47.144320 merkle-py-1.2.2/src/merklepy/
+-rw-r--r--   0 cyrildever   (501) staff       (20)        0 2022-03-21 11:01:19.000000 merkle-py-1.2.2/src/merklepy/__init__.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      657 2022-04-04 08:47:17.000000 merkle-py-1.2.2/src/merklepy/exception.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      971 2022-04-04 08:47:17.000000 merkle-py-1.2.2/src/merklepy/hash.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      843 2022-04-04 08:47:17.000000 merkle-py-1.2.2/src/merklepy/options.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     1207 2022-04-04 08:47:17.000000 merkle-py-1.2.2/src/merklepy/path.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2287 2022-04-04 10:31:42.000000 merkle-py-1.2.2/src/merklepy/proof.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     6813 2022-04-04 08:47:17.000000 merkle-py-1.2.2/src/merklepy/tree.py
+drwxr-xr-x   0 cyrildever   (501) staff       (20)        0 2023-04-17 07:03:47.147168 merkle-py-1.2.2/tests/
+-rw-r--r--   0 cyrildever   (501) staff       (20)     2319 2022-04-04 08:47:17.000000 merkle-py-1.2.2/tests/test_hash.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      523 2022-04-04 08:47:17.000000 merkle-py-1.2.2/tests/test_options.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)      875 2022-04-04 08:47:17.000000 merkle-py-1.2.2/tests/test_path.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     1749 2022-04-04 08:47:17.000000 merkle-py-1.2.2/tests/test_proof.py
+-rw-r--r--   0 cyrildever   (501) staff       (20)     5595 2022-04-04 08:47:17.000000 merkle-py-1.2.2/tests/test_tree.py
```

### Comparing `merkle-py-1.2.1/PKG-INFO` & `merkle-py-1.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: merkle-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Merkle tree for Python
-Home-page: https://github.com/cyrildever/merkle-trees/packages/py
+Home-page: https://github.com/cyrildever/merkle-trees/tree/master/packages/py
 Author: Cyril Dever
 Project-URL: Bug Tracker, https://github.com/cyrildever/merkle-trees/issues
-Keywords: python,merkle-tree
+Keywords: python,merkle-tree,merkle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # merkle-py
 _Python implementation of Merkle tree_
 
+![Github tag (latest by date)](https://img.shields.io/github/v/tag/cyrildever/merkle-trees)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/merkle-py)
+![Github last commit](https://img.shields.io/github/last-commit/cyrildever/merkle-trees)
+![Github issues](https://img.shields.io/github/issues/cyrildever/merkle-trees)
+![PyPI - License](https://img.shields.io/pypi/l/merkle-py)
+
 This library defines my special implementation in Python of the notorious Merkle trees. Feel free to use it (with the appropriate credits).
 
 Other implementations include: [Go](../go/README.md), [Scala](../scala/README.md) and [TypeScript](../ts/README.md).
 
-
 ### Usage
 
 ```console
 $ pip install merkle-py
 ```
 
 Here are some simple examples of how it works:
@@ -72,13 +77,13 @@
 ```console
 $ python3 -m unittest discover
 ```
 
 
 ### License
 
-This library is distributed under an MIT license.
+This library is distributed under a MIT license. \
 See the [LICENSE](LICENSE) file.
 
 
 <hr />
 &copy; 2022-2023 Cyril Dever. All rights reserved.
```

### Comparing `merkle-py-1.2.1/README.md` & `merkle-py-1.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # merkle-py
 _Python implementation of Merkle tree_
 
+![Github tag (latest by date)](https://img.shields.io/github/v/tag/cyrildever/merkle-trees)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/merkle-py)
+![Github last commit](https://img.shields.io/github/last-commit/cyrildever/merkle-trees)
+![Github issues](https://img.shields.io/github/issues/cyrildever/merkle-trees)
+![PyPI - License](https://img.shields.io/pypi/l/merkle-py)
+
 This library defines my special implementation in Python of the notorious Merkle trees. Feel free to use it (with the appropriate credits).
 
 Other implementations include: [Go](../go/README.md), [Scala](../scala/README.md) and [TypeScript](../ts/README.md).
 
-
 ### Usage
 
 ```console
 $ pip install merkle-py
 ```
 
 Here are some simple examples of how it works:
@@ -58,13 +63,13 @@
 ```console
 $ python3 -m unittest discover
 ```
 
 
 ### License
 
-This library is distributed under an MIT license.
+This library is distributed under a MIT license. \
 See the [LICENSE](LICENSE) file.
 
 
 <hr />
 &copy; 2022-2023 Cyril Dever. All rights reserved.
```

### Comparing `merkle-py-1.2.1/setup.py` & `merkle-py-1.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="merkle-py",
-    version="1.2.1",
+    version="1.2.2",
     author="Cyril Dever",
     author_mail="cdever@pep-s.com",
     description="Merkle tree for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/cyrildever/merkle-trees/packages/py",
+    url="https://github.com/cyrildever/merkle-trees/tree/master/packages/py",
     project_urls={
         "Bug Tracker": "https://github.com/cyrildever/merkle-trees/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=[
         "python",
         "merkle-tree",
+        "merkle",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

### Comparing `merkle-py-1.2.1/src/merkle_py.egg-info/PKG-INFO` & `merkle-py-1.2.2/src/merkle_py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: merkle-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: Merkle tree for Python
-Home-page: https://github.com/cyrildever/merkle-trees/packages/py
+Home-page: https://github.com/cyrildever/merkle-trees/tree/master/packages/py
 Author: Cyril Dever
 Project-URL: Bug Tracker, https://github.com/cyrildever/merkle-trees/issues
-Keywords: python,merkle-tree
+Keywords: python,merkle-tree,merkle
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # merkle-py
 _Python implementation of Merkle tree_
 
+![Github tag (latest by date)](https://img.shields.io/github/v/tag/cyrildever/merkle-trees)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/merkle-py)
+![Github last commit](https://img.shields.io/github/last-commit/cyrildever/merkle-trees)
+![Github issues](https://img.shields.io/github/issues/cyrildever/merkle-trees)
+![PyPI - License](https://img.shields.io/pypi/l/merkle-py)
+
 This library defines my special implementation in Python of the notorious Merkle trees. Feel free to use it (with the appropriate credits).
 
 Other implementations include: [Go](../go/README.md), [Scala](../scala/README.md) and [TypeScript](../ts/README.md).
 
-
 ### Usage
 
 ```console
 $ pip install merkle-py
 ```
 
 Here are some simple examples of how it works:
@@ -72,13 +77,13 @@
 ```console
 $ python3 -m unittest discover
 ```
 
 
 ### License
 
-This library is distributed under an MIT license.
+This library is distributed under a MIT license. \
 See the [LICENSE](LICENSE) file.
 
 
 <hr />
 &copy; 2022-2023 Cyril Dever. All rights reserved.
```

### Comparing `merkle-py-1.2.1/src/merklepy/exception.py` & `merkle-py-1.2.2/src/merklepy/exception.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/src/merklepy/hash.py` & `merkle-py-1.2.2/src/merklepy/hash.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/src/merklepy/options.py` & `merkle-py-1.2.2/src/merklepy/options.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/src/merklepy/path.py` & `merkle-py-1.2.2/src/merklepy/path.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/src/merklepy/proof.py` & `merkle-py-1.2.2/src/merklepy/proof.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/src/merklepy/tree.py` & `merkle-py-1.2.2/src/merklepy/tree.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/tests/test_hash.py` & `merkle-py-1.2.2/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/tests/test_options.py` & `merkle-py-1.2.2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/tests/test_path.py` & `merkle-py-1.2.2/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/tests/test_proof.py` & `merkle-py-1.2.2/tests/test_proof.py`

 * *Files identical despite different names*

### Comparing `merkle-py-1.2.1/tests/test_tree.py` & `merkle-py-1.2.2/tests/test_tree.py`

 * *Files identical despite different names*

